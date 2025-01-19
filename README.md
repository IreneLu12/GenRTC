# GenRTC
Perceptual comparison for paper titled "**GenRTC: Low Bandwidth Video Conferencing System with Generative Face Coding**".
In this perceptual experiment, frame dropping is introduced to maintain playback synchronization, it results in substantial content loss and stuttering due to excessive frame loss. Note that timeout frames are marked as "Timeout! Drop!", and frames dropped due to webrtc internal bitrate requirement detection mechanism are marked as "Loss".
Based on below comparison, it shows that GenRTC, with its more effective adaptive encoder and precise bandwidth estimator, efficiently handles network fluctuations, providing a more stable transmission. At the same time, GenRTC maintains relatively high perceptual quality. 


## Case 1
Baseline:
- missrate = 0.54 Vmaf = 86.74, PSNR = 42.02 SSIM = 0.99, LPIPS = 0.037

Ours:
- missrate = 0.04 Vmaf = 77.43, PSNR = 38.69 SSIM = 0.96, LPIPS = 0.055

https://github.com/user-attachments/assets/6c52c9d8-1f89-4a1c-a102-0a44f56b72b8


## Case 2
Baseline:
- missrate = 0.32 Vmaf = 87.09, PSNR = 32.17 SSIM = 0.97, LPIPS = 0.031

Ours:
- missrate = 0.05 Vmaf = 79.51, PSNR = 29.69 SSIM = 0.95, LPIPS = 0.045

https://github.com/user-attachments/assets/bd607e75-48a8-48ae-a033-49f14551a03e
