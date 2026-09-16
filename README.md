# Cutout BiRefNet portrait

Browser-compatible ONNX model for https://bigrooo.github.io/cutout-web/.
Source: danielgatis/rembg v0.0.0, BiRefNet-portrait-epoch_150.onnx. BiRefNet is MIT licensed.

Modified export: prepare_browser_model.py fuses expanded deformable convolution
into native ONNX DeformConv (opset 19). Original FP32 trained weights and 1024
input resolution are preserved. Requires ONNX Runtime Web 1.30 or newer.
CI verifies source and final SHA-256; model binaries are deployed as Pages
artifacts, not committed to Git. No images are uploaded here.
