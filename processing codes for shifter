import mqtt.*;

MQTTClient client;

void setup() {
  client = new MQTTClient(this);
  client.connect("mqtt://datt3700:datt3700experiments@datt3700.cloud.shiftr.io", "Yuxuan");
  client.subscribe("Hello");
}

void draw() {}

void keyPressed() {
  client.publish("hello", "OwO");
}

void messageReceived(String topic, byte[] payload) {
  println( topic + ": " + new String(payload));
}
