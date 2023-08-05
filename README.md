# nnU-Net For PyTorch

Training command:
```
python main.py --brats --deep_supervision --depth 6 --filters 64 96 128 192 256 384 512 --min_fmap 2 --scheduler --learning_rate 0.0003 --epochs 200 --fold 0 --amp --gpus 2 --task 11 --save_ckpt --data /raid/compass/mobarak/datasets/brats2023/train/train_valid/11_3d --results /raid/compass/mobarak/datasets/brats2023/train/train_valid --ckpt_store_dir ckpt_ours --batch_size 4 --val_batch_size 10
```
