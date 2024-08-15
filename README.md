# ESP32-CAM
Usar versiones de placa esp32 by Espressif Systems <br>
Libreria ESP32-CAM por: <p><a href="https://github.com/yoursunny">yoursunny<p><br>
2.0.2  -> Trabajar con todas las placas ESP32 (incluyendo OpenCV para ESP32-CAM)<br>
1.0.6 -> Trabajar con ESP32-CAM sin OpenCV (CameraWebServer)<br>
Cambios en la libreria para ESP32-CAM en 2.0.2 en esp32cam/src/internal/config.cpp<br>
Config::setPins(const Pins& pins) {<br>
    .<br>
    .<br>
    .<br>
  m_cfg->pin_sccb_sda = pins.SDA; -> m_cfg->pin_sscb_sda = pins.SDA;<br>
  m_cfg->pin_sccb_scl = pins.SCL; -> m_cfg->pin_sscb_scl = pins.SCL;<br>
    .<br>
    .<br>
    .<br>
}