--------------
DFU Mode
Using the Python HID Library, this is effortless. The important thing to know is the dfu_payload which get’s send to the device.
```
dfu_payload = [0, 85, 170, 1, 2, 3, 4, 170, 85]
device = hid.device()
device.open(vendor_id,product_id)
print(f"HID: Found Device: {device.get_manufacturer_string()} {device.get_product_string()}")
data = bytearray(byte_array_left_pad([0, 33, 9, 0, 2, 1, 0, 64, 0], 0, 65))
buffer_payload = bytearray(byte_array_left_pad(dfu_payload, 0, 65))
device.write(data)
try:
	device.write(buffer_payload)
except Exception:
	print("\nCommunication Error or DFU Success...")
```
You can now flash new firmware on the chip.
https://nv1t.github.io/blog/kekz-headphones/
--------------
https://vi.aliexpress.com/item/1005007090348648.html
--------------
https://doc.zh-jieli.com/AC79/zh-cn/release_v1.1.0/getting_started/preparation/update.html
--------------
https://gitlab.zh-jieli.com/soundbox/novisualization/ac695n_soundbox_sdk
--------------
https://github.com/kagaimiq/jl-misctools
--------------
https://electronics.stackexchange.com/questions/734433/jieli-tech-ac6955f4-bluetooth-ic-programming
--------------

JL upgrade tool with USB serial port debugging, USB compulsory download, compulsory burner

https://vi.aliexpress.com/item/4000012929223.html

![Screenshot 2025-01-05 at 7 39 15 am](https://github.com/user-attachments/assets/e4694099-f9a1-4fc2-987b-ca6623be2a66)

--------------
Jieli, Bluetooth Chip Activator USB Forced Bulk Upgrade Tool AC69XX Series Development Board Downloader

https://vi.aliexpress.com/i/1005008004492960.html

![Screenshot 2025-01-05 at 7 41 57 am](https://github.com/user-attachments/assets/d2875735-d809-48d7-9d8b-67fb80bb4f3e)
![Screenshot 2025-01-05 at 7 42 00 am](https://github.com/user-attachments/assets/9735ce24-41f0-491d-b624-bd017e38bbb1)
![Screenshot 2025-01-05 at 7 42 12 am](https://github.com/user-attachments/assets/b2acf415-4c0e-49f9-ab06-9db59963b438)
![Screenshot 2025-01-05 at 7 42 17 am](https://github.com/user-attachments/assets/4dc53565-2623-4640-b1e2-51bb05b16b6c)

