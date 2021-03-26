# 2420_week11

Installation Steps

1. Clone the github rep: "git clone https://github.com/Markus-uss/2420_week11.git"

2. Move or copy the weather.service and weather.timer into /etc/systemd/system using: "-cp weather.service /etc/systemd/system" or "-mv weather.service /etc/systemd/system". Do the same for weather.timer

3. Run the command: "sudo systemctl daemon-reload", this will update previous configurations of systemd.

4. Start the hourly loop using: "sudo systemctl start /etc/systemd/system/weather.timer"

5. Start the service script using: "sudo systemctl start /etc/systemd/system/weather.service"

6. The weather bash script will now generate a weather report every hour in the directory it is located in.
