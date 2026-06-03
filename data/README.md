# Dataset: LOL-v1 + LOL-v2-real

Dataset combinado de pares de imágenes para la tarea de **low-light image enhancement**.
Cada par consiste en una imagen de baja iluminación (`low`) y su contraparte de iluminación
normal (`high`), capturadas en las mismas condiciones de escena.

## Fuentes

| Dataset | Fuente | Link |
|---|---|---|
| LOL-v1 | Kaggle | https://www.kaggle.com/datasets/soumikrakshit/lol-dataset |
| LOL-v2-real | HuggingFace | https://huggingface.co/datasets/okhater/lolv2-real |

## Estructura esperada

    data/
    ├── lol-v1/
    │   ├── our485/
    │   │   ├── low/
    │   │   └── high/
    │   └── eval15/
    │       ├── low/
    │       └── high/
    └── lolv2-real/
        ├── Train/
        │   ├── Input/
        │   └── GT/
        └── Test/
            ├── Input/
            └── GT/

## Descarga

Ver celda **"Descarga del dataset"** en el notebook. Requiere:
- Credenciales de Kaggle (`KAGGLE_USERNAME` y `KAGGLE_KEY`)
- Cuenta en HuggingFace (acceso público, no requiere token)

## Estadísticas

| Split | Pares |
|---|---|
| Train | 939 |
| Val | 117 |
| Test | 118 |
| **Total** | **1174** |

## Papers de referencia

- **LOL-v1**: Wei et al., *Deep Retinex Decomposition for Low-Light Enhancement*, BMVC 2018
- **LOL-v2**: Yang et al., *Sparse Gradient Regularized Deep Retinex Network*, TIP 2021
- **Modelo de referencia**: Cai et al., *Retinexformer: One-stage Retinex-based Transformer for Low-light Image Enhancement*, ICCV 2023