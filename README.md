# nnU-Net For PyTorch

Training Command:
```
python main.py --brats --deep_supervision --depth 6 --filters 64 96 128 192 256 384 512 --min_fmap 2 --scheduler --learning_rate 0.0003 --epochs 200 --fold 1 --amp --gpus 2 --task 11 --save_ckpt --data /raid/compass/mobarak/datasets/brats2023/train/train_valid/11_3d --results /raid/compass/mobarak/datasets/brats2023/train/train_valid --ckpt_store_dir ckpt_ours --batch_size 4 --val_batch_size 10
```
Official Validation Command (must be done on single GPU):
```
python main.py --brats --deep_supervision --depth 6 --filters 64 96 128 192 256 384 512 --min_fmap 2 --gpus 1 --amp --save_preds --exec_mode predict  --data /raid/compass/mobarak/datasets/brats2023/valid/official_valid/12_3d/test --ckpt_path /raid/compass/mobarak/brats/nnUNet_BraTS/ckpt_ours/checkpoints/epoch=131-dice=90.34.ckpt --tta --results /raid/compass/mobarak/datasets/brats2023/valid/official_valid/
```
```
python main.py --brats --deep_supervision --depth 6 --filters 64 96 128 192 256 384 512 --min_fmap 2 --gpus 1 --amp --save_preds --exec_mode predict  --data /raid/compass/mobarak/datasets/brats2023/valid/official_valid/12_3d/test --ckpt_path /raid/compass/mobarak/brats/nnUNet_BraTS/ckpt_ours/checkpoints/epoch=173-dice=90.28.ckpt --tta --results /raid/compass/mobarak/datasets/brats2023/valid/official_valid/
```
```
python main.py --brats --deep_supervision --depth 6 --filters 64 96 128 192 256 384 512 --min_fmap 2 --gpus 1 --amp --save_preds --exec_mode predict  --data /raid/compass/mobarak/datasets/brats2023/valid/official_valid/12_3d/test --ckpt_path /raid/compass/mobarak/brats/nnUNet_BraTS/ckpt_ours/checkpoints/epoch=195-dice=91.42.ckpt --tta --results /raid/compass/mobarak/datasets/brats2023/valid/official_valid/
```
```
python main.py --brats --deep_supervision --depth 6 --filters 64 96 128 192 256 384 512 --min_fmap 2 --gpus 1 --amp --save_preds --exec_mode predict  --data /raid/compass/mobarak/datasets/brats2023/valid/official_valid/12_3d/test --ckpt_path /raid/compass/mobarak/brats/nnUNet_BraTS/ckpt_ours/checkpoints/epoch=166-dice=90.83.ckpt --tta --results /raid/compass/mobarak/datasets/brats2023/valid/official_valid/
```
```
python main.py --brats --deep_supervision --depth 6 --filters 64 96 128 192 256 384 512 --min_fmap 2 --gpus 1 --amp --save_preds --exec_mode predict  --data /raid/compass/mobarak/datasets/brats2023/valid/official_valid/12_3d/test --ckpt_path /raid/compass/mobarak/brats/nnUNet_BraTS/ckpt_ours/checkpoints/epoch=72-dice=89.73.ckpt --tta --results /raid/compass/mobarak/datasets/brats2023/valid/official_valid/
```
