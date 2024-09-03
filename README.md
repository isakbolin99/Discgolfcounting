# Discgolfcounting

## Description
The idea of discgolfcounting was born in 2019 when I had no idea about how many players were using my newly built disc golf course: https://udisc.com/courses/tjaerna-sandtag-ZUlv. Since disc golf is usually free to play, it is hard to estimate the number of players in my city and the rest of the country. To solve this problem I built a footfall counter that counts all the players on the course. Data is sent via the IoT-friendly NB-IoT network to a cloud-based SQL database. Data is displayed on a website (discgolfcounting.com) to provide statistics to players, companies, and club owners.

## Footfall counter
The counter is placed by a narrow walk path on the course. The Device is powered by standard AA batteries. To save power, the device is put into sleep-mode. It is woken up by an interrupt triggered by the PIR sensor in the device. Thereafter, the number of players in the group is counted with the help of an ultrasonic distance sensor. Once every hour, data is sent via NB-IoT to a cloud-based database before the statistics are provided for players on discgolfcounting.com.



