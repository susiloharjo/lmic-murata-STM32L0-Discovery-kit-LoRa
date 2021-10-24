# lmic-murata-STM32L0-Discovery-kit-LoRa

HOW to use lmic at https://www.st.com/en/evaluation-tools/b-l072z-lrwan1.html


## Add this at setup
SPI.setMOSI(PA7);
SPI.setMISO(PA6);
SPI.setSCLK(PB3);

##  Pin mapping

const lmic_pinmap lmic_pins = {
  .nss = PA15,
  .rxtx = LMIC_UNUSED_PIN,
  .rst = PC0,
  .dio = {PB4, PB1, PB0},
};
