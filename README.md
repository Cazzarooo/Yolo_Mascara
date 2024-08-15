# YOLO Mascara Detection

Este projeto utiliza o modelo YOLOv5 para detecção de máscaras faciais. Ele foi desenvolvido para identificar se uma pessoa está utilizando uma máscara facial corretamente.

Instalação

Pré-requisitos
É necessário ter um ambiente com suporte a GPU para melhor desempenho.
Recomendado utilizar Google Colab com acelerador de hardware GPU.

# Passos para Configuração:

1 - Clone o repositório do YOLOv5:
`!git clone https://github.com/ultralytics/yolov5
%cd yolov5`

2 - Faça o reset do repositório para uma versão específica:
`!git reset --hard 064365d8683fd002e9ad789c1e91fa3d021b44f0`

3 - Instale as dependências necessárias:
`!pip install -qr requirements.txt`

# Uso

Após configurar o ambiente, você pode realizar a inferência em imagens locais para detectar a presença de máscaras faciais.

Exemplo de Uso

1- Inicialize o cliente de inferência:
`from inference_sdk import InferenceHTTPClient`

`CLIENT = InferenceHTTPClient(
    api_url="https://detect.roboflow.com",
    api_key="sua_api_key_aqui"
)`

2 - Realize a inferência sobre uma imagem local:
`result = CLIENT.infer("/caminho/para/sua/imagem.png", model_id="mascara-yw6sr/1")`

Contribuição
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.



