## EXAMPLES

The examples show you how to use LuaNode.

* **wifi_scan**: Scan all APs around ESP32 device.
* **raw_flash_rw**: Read write ESP32 flash directly without file system.
* **simple_http_server**: Create a simple http server on ESP32. To test this 
			example, build it follow the next section, and then 
			connect to the AP established on ESP32 using your phone. 
			The AP named as `DOIT_XXXX`. When connect to ESP32 device, 
			open `192.168.4.1` on browser, you'll see a test page, 
			which echo `This is a test`, returned 
			from ESP32.
* **tcp_server_espconn**: A simple tcp server sample create with _espconn_. The server 
		listen port 11000. When client send data, the server will print the data.
* **tcp_client_espconn**: A tcp client create with _espconn_. To test this sample, make 
		sure the client and the server connected with the same network segment, 
		and the server listen the port 11000, than the server can receive data sent 
		from client.
* **dns_resolver**: A DNS resolver sample. To test this sample, connect your phone or 
		computer to ESP32 which run this sample, and then open any link in the browser.
		the return page will be a test page.
* **udp_server_espconn**: A udp server sample.
* **udp_broadcast**: A UDP broadcast sample create with _espconn_. In this sample, we create 
		a task to broadcast UDP message repeatedly. The remote port is set to 11000. 
		If you create a UDP server to listen the port, you'll receive the message sent from 
		ESP32 device. Don't forget to modified the macro EXAMPLE_WIFI_SSID and EXAMPLE_WIFI_PASS to 
		valid value.
* **telnet_server**: A simple telnet server sample. When you connect with ESP32 using telnet, and then 
		input command `hello`, it will echo `hello back`.
* **lwip_raw_api**: A RAW API sample. Show you how to use LwIP RAW API.
* **easy_mem**: A sample show you to use _easy_mem_, the memory manager.
* **bluetooth_scanner**: A sample show you how to scan BLE device. To test this sample, you 
		can use two ESP32 device, say A and B. A flashed the _ble_adv_ which is an example contained in _esp-idf_, 
		B flashed this sample. Then you can see B output the scan results, which list A. The other available 
		BLE device will be also listed in the results.
* **test_spiffs**: A test sample for SPIFFS.
* **camera**: A sample to show you how to use ESP32 to control a camera
* **lcd_nokia5110_driver**: A sample to show how to drive _Nokia5110_ LCD. The sample output some 
		characters to LCD.

* **ble_led_control**: A sample to show how to create BLE client and BLE server. In this sample, the 
		client send notify to server each 2 seconds. When the server receives the notification, 
		the server will turn on/off the blue LED on board according to the notification value. 
		To test this sample, you have to prepare two ESP32 dev-board.

## HOW TO BUILD THE EXAMPLES

Copy the app_main.c within each example to the `main` folder within LuaNode32,
and then run `./build.sh` to build LuaNode.
