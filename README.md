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
  * 
  
## Honeypot 2 (mhn-5):
* Type:
  * Snort
* Data collected:
  * Number of attacks: 821
  * Origin Sources: USA, Russia, China, Romania, 
  * 
  
## Honeypot 3 (mhn-6):
* Type:
  * Suricata
* Data collected:
  * Number of attacks: 4,143
  * Origin Sources: USA, Germany, Russia, Netherlands, Sweden, China, etc.
  * Payload Samples Collected: About 6,374
    *
## Unanswered Question
* At some around the half way point of 2 days the number of attacks began to stagnate. On the morning of 4-16 I noticed that the MHN dashboard was displaying a lesser amount of cumulative attacks.
  * 8,151 attacks logged on the evening of 4-15
  * 7,837 attacks logged on the morning of 4-16
* My only explanation as to why this may be occuring is because the MHN Server is recognizing duplicated data and removing it from the pool of data. I also noticed that the MHN Server updates the information on it every so often (hours) however I'm not sure what the exact number is. I noticed this, because I originally had 2 other sensors on two seperate VMs set up. They remained the MHN Server home page for a couple of hours until I removed them and destroyed the VMs they were on and noticed that they were suddenly not there anymore. 
 
# Resources
[Sensor Types](https://github.com/threatstream/mhn/wiki/List-of-Supported-Sensors)
