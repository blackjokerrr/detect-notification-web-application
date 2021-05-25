<h1>Raspberry Pi Notification with HIVEMQ</h1>
<li>เป็นโปรเจคที่ใช้ Raspberry Pi กับ Raspberry Pi 8MP NOIR Camera Board V2 ทำหน้าที่คอยแจ้งเตือนว่ามีการ Detect อะไรบ้างโดยจะใช้ Library อย่าง Tensorflow เข้ามาช่วยเพื่อให้ Raspberry Pi มีความฉลาดมากขึ้นเมื่อ Detect อะไรได้จะทำการแสดงผลผ่าน HIVEMQ โดยจะคุยกันผ่าน Protocal MQTT</li>
<h1>Equipment</h1>
<li>Raspberry Pi</li>
<li>Raspberry Pi 8MP NOIR Camera Board V2</li>
<h1>Software</h1>
<li><a href = 'https://www.putty.org/'>PuTTY</a></li>
<li><a href = 'http://www.hivemq.com/demos/websocket-client/'>HIVEMQ</a></li>
<h1>Library</h1>
<li><a href = 'https://www.eclipse.org/paho/index.php?page=clients/python/index.php'>Paho Python</a></li>
<li><a href = 'https://www.tensorflow.org/lite'>Tensorflow</a></li>
<li><a href = 'https://opencv.org/'>Opencv</a></li>

<h1>Install on Raspberry Pi</h1>

1. Clone github repo

```
git clone https://github.com/blackjokerrr/detect-notification-with-hivemq.git
```

2. move to detect-notification-with-hivemq folder

```
cd detect-notification-with-hivemq
```

3. activate env

```
source tflite1-env/bin/activate
```

4. Run

```
python3 detect.py --modeldir=Sample_TFLite_model
```

5. Open HIVEMQ

6. Subscribe Topic

```
raspberrypi/project
```