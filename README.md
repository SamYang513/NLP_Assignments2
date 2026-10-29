# 中文句子情緒分類

## 訓練資料來源

- ChatGPT 自動生成

## 基礎模型

```
Qwen/Qwen2.5-0.5B-Instruct
```


## 說明

1. 專案介紹

本專案使用 

```
Qwen/Qwen2.5-0.5B-Instruct
```

對lora模型進行微調 改了上下文參照由7句改到10句 資料來源使用chatGPT生成的土味情話 <<chat.jsonl>> 每句對話超過三段


## 執行方法


# 1. 準備 SFT 資料

python prepare_chat_data.py

# 2. 執行 QLoRA 微調

python train_qlora.py

# 3. 畫出 Loss 曲線

python plot_loss.py

# 4. 多輪對話測試

python infer_lora_chat.py

## 其它你想要補充標題和內容

訓練模型結果不佳 對著資料集的問題問了一遍答出來的結果卻完全不一樣 土味情人變成奶油小生 說話都客氣了很多
