# 静止画新環境

Paperspace のノートブック作成画面で「Start from Scratch」を選択して、

「View advanced options」をクリックして、コンテナ名(Container⇒Name)として

javacommons/paperspace-std:v2025.0517.1811 (タイムゾーン: UTC)

または

javacommons/paperspace-std:v2025.0517.1811-JST (タイムゾーン: JST (Asia/Tokyo))

を指定して「START NOTEBOOK」をクリックします。

各 ipynb のダウンロードは、Paperspace のターミナルから以下のようにしてダウンロードできます。

ターミナルからは以下でダウンロードできます。

```
cd /notebooks
wget https://github.com/paperspace-newenv/ipynb/raw/main/a1111.ipynb
wget https://github.com/paperspace-newenv/ipynb/raw/main/comfyui.ipynb
wget https://github.com/paperspace-newenv/ipynb/raw/main/reforge.ipynb
```

----

## ComfyUI とA1111 の共存に関してです。(mush さんより)

モデル（チェックポイント）、LoRa、VAE などを共有するための設定ですが、ComfyUIのインストールディレクトリにある extra_model_paths.yaml.example を extra_model_paths.yaml にリネームし、base_path: を A1111 のディレクトリパス（/notebooks/stable-diffusion-webui/）に変更するだけで簡単に設定できます。
