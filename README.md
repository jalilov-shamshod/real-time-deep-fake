![demo-gif](demo.gif)

## Ogohlantirish
Ushbu dasturiy taʼminot o‘sib borayotgan sunʼiy idrok jamiyatiga hissa qo‘shish uchun yaratilgan. Dasturchilar uni axloqsiz tasvirlarda foydalanilishi, qonunlardan tashqari maqsadlarda qo‘llanilishi uchun javobgarlikni bo‘yinga olmaydi.Shaxsni yuzidan foydalanmoqchi bo‘lsangiz ularni roziligini oling, shuningdek materialni internetga joylashtirganingizda uni deep fake(soxta) ekanini aniq ko‘rsatib qo‘ying. Dasturchilar taʼminotni ishlab chiquvchilar oxirgi foydalanuvchilarning harakatlari uchun javobgar bo‘lmaydilar.

## Uni qanday o'rnataman?

### Asosiy: Loyiha katta ehtimollikda sizni kompyuteringizda ishlaydi, ammo u asta ishlashi ham mumkin.

#### 1.O'rnatishdan oldin sizga zarur bo'ladi
-   python (3.10 tavsiya qilinadi)
-   pip
-   git
-   [ffmpeg](https://www.youtube.com/watch?v=OlNWCpFdVMA) 
-   [visual studio 2022 runtimes (windows)](https://visualstudio.microsoft.com/visual-cpp-build-tools/)

#### 2. Loyihani klonlang
    https://github.com/jalilov-shamshod/real-time-deep-fake.git

#### 3. Zarur qaramliklarni o'rnating
Virtual muhit -  `venv` dan foydalanish tavsiya etiladi.
```
pip install -r requirements.txt
```
##### Yakunlandi!!! Agar sizda GPU bo'lmasa, "python run.py" buyrug'i yordamida loyihani ishga tushirishingiz mumkin. Yodda tutingki, dastur birinchi marta ishga tushganda u ba'zi modellarni yuklab oladi.

//------------------------------------------------------------------------------------//

### *GPU tezlatishidan foydalanmoqchi bo'lsangiz:

### CUDA Ijrochi Provayderi (Nvidia):

1.  O'rnating  [CUDA Toolkit 11.8](https://developer.nvidia.com/cuda-11-8-0-download-archive)
    
2.  Zarur qaramlikni o'rnating:

```
pip uninstall onnxruntime onnxruntime-gpu
pip install onnxruntime-gpu==1.16.3

```

3. Provayder mavjud bo'lsa:

```
python run.py --execution-provider cuda

```

### [](https://github.com/s0md3v/roop/wiki/2.-Acceleration#coreml-execution-provider-apple-silicon)CoreML Ijrochi Provayderi (Apple Silicon)

1.  Zarur qaramlikni o'rnating:

```
pip uninstall onnxruntime onnxruntime-silicon
pip install onnxruntime-silicon==1.13.1

```

2.  Provayder mavjud bo'lsa:

```
python run.py --execution-provider coreml

```

### [](https://github.com/s0md3v/roop/wiki/2.-Acceleration#coreml-execution-provider-apple-legacy)CoreML Ijrochi Provayderi (Apple Legacy)

1.  Zarur qaramlikni o'rnating:

```
pip uninstall onnxruntime onnxruntime-coreml
pip install onnxruntime-coreml==1.13.1

```

2.  Provayder mavjud bo'lsa:

```
python run.py --execution-provider coreml

```

### [](https://github.com/s0md3v/roop/wiki/2.-Acceleration#directml-execution-provider-windows)DirectML Ijrochi Provayderi (Windows)

1. Zarur qaramlikni o'rnating:

```
pip uninstall onnxruntime onnxruntime-directml
pip install onnxruntime-directml==1.15.1

```

2.  Provayder mavjud bo'lsa:

```
python run.py --execution-provider directml

```

### [](https://github.com/s0md3v/roop/wiki/2.-Acceleration#openvino-execution-provider-intel)OpenVINO™ Ijrochi Provayderi (Intel)

1.  Zarur qaramlikni o'rnating:

```
pip uninstall onnxruntime onnxruntime-openvino
pip install onnxruntime-openvino==1.15.0

```

2.  Provayder mavjud bo'lsa:

```
python run.py --execution-provider openvino
```

## Muallif
- [hacksider](https://github.com/hacksider/Deep-Live-Cam): mehnati uchun tashakkur bildirib qolamiz.
