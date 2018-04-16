# Week-9

## Attacking The Honeypot ![Attack](https://github.com/0v3rride/Week-9/blob/master/attack.gif)
## Threat Map ![Threat Map](https://github.com/0v3rride/Week-9/blob/master/Threat_Map.gif)
## Overall Stats ![Stats](https://github.com/0v3rride/Week-9/blob/master/Overall_stats.gif)
## Detailed Attack Data ![Attack Data](https://github.com/0v3rride/Week-9/blob/master/Detailed_Attack_Data.gif)

## Information:
* Pots were setup and ran on 4-14 until 4-16.
 * I noticed that no new data was being collected by any of them on the morning of 4-16.
 
## Honeypot 1 (mhn-4):
* Type:
  * Dionaea with HTTP 
* Data collected:
  * Number of attacks: 3,169
  * Origin Sources: USA, Canada, Mexico, Brazil, United Kingdom, France, Netherlands, Croatia, Germany, Poland, Bulgaria, Egypt, Australia, Japan, Indonesia, China, Vietnam, Iran, Turkey, South Korea, Ukraine, Romania, Switzerland, Russia, etc.
  * No payload or signatures samples were collected by this sensor.
  
## Honeypot 2 (mhn-5):
* Type:
  * Snort
* Data collected:
  * Number of attacks: 821
  * Origin Sources: USA, Russia, China, Romania, France, Germany, etc.
  * Payload/Signature Samples Collected: About 1,410
    * Some Samples:
      * ET DROP Spamhaus DROP Listed Traffic Inbound group 33
      * ET CINS Active Threat Intelligence Poor Reputation IP TCP group 4
      * ET DROP Dshield Block Listed Source group 1
  
## Honeypot 3 (mhn-6):
* Type:
  * Suricata
* Data collected:
  * Number of attacks: 4,143
  * Origin Sources: USA, Germany, Russia, Netherlands, Sweden, China, etc.
  * Payload/Signature Samples Collected: About 6,374
    * Some Samples:
      * ET POLICY Python-urllib/ Suspicious User Agent
      * ET CINS Active Threat Intelligence Poor Reputation IP TCP group 4
      * ET DROP Dshield Block Listed Source group 1
     
## Unanswered Question
* At some time around the half way point of between 48 hours, the number of attacks being collected began to stagnate. On the morning of 4-16 I noticed that the MHN dashboard was displaying a lesser amount of cumulative attacks than what was displayed the previous evening.
  * 8,151 attacks logged on the evening of 4-15
  * 7,837 attacks logged on the morning of 4-16
* My only explanation as to why this may be occuring is because the MHN Server is recognizing duplicated data and removing it from the pool of data. I also noticed that the MHN Server updates the information on it every so often (hours) however I'm not sure what the exact number is. I noticed this, because I originally had 2 other sensors on two seperate VMs set up. They remained on my MHN Server's home page for a couple of hours until I removed them and destroyed the VMs they were on and noticed that they were suddenly gone a couple of hours later. 
 
# Resources
[Sensor Types](https://github.com/threatstream/mhn/wiki/List-of-Supported-Sensors)
