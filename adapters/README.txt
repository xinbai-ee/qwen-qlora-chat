本目录用于存放训练好的 QLoRA 适配器。

子目录 qwen2.5-7b-qlora/
  训练成功完成后，脚本会把以下文件写到这里：
  - adapter_config.json
  - adapter_model.safetensors
  （或 checkpoint-xxx 文件夹）

若该子目录目前是空的：
  说明训练尚未成功跑完，或上次训练中断/报错了。
  请重新运行训练：
    双击「从chat训练.bat」
    或在项目目录执行：python scripts/train_qlora.py
  等训练跑完后，这里会自动出现上述文件，后端和推理脚本会加载它们。
