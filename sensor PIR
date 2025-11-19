const int pirPin = D1;  // Pin untuk sensor PIR
const int ledPin = D2;  // Pin untuk LED

void setup() {
  Serial.begin(115200);  // Memulai komunikasi serial
  pinMode(pirPin, INPUT);  // Set pin PIR sebagai input
  pinMode(ledPin, OUTPUT);  // Set pin LED sebagai output
}

void loop() {
  int pirState = digitalRead(pirPin);  // Membaca status sensor PIR

  if (pirState == HIGH) {  // Jika gerakan terdeteksi
    digitalWrite(ledPin, HIGH);  // Nyalakan LED
    Serial.println("Gerakan terdeteksi!");  // Tampilkan pesan di Serial Monitor
  } else {
    digitalWrite(ledPin, LOW);  // Matikan LED
    Serial.println("Tidak ada gerakan.");  // Tampilkan pesan di Serial Monitor
  }

  delay(200);  // Delay untuk menghindari pembacaan yang terlalu cepat
}
