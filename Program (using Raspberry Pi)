//LED using raspberry pi 
import RPi.GPIO as GPIO   
 import time   
 led_array = [ 11, 12, 13, 15, 16, 18, 22, 7];   
 blink_delay = 0.5   
 try:   
   GPIO.setmode(GPIO.BOARD)   
   for i in range(0,8):   
     GPIO.setup(led_array[i], GPIO.OUT)   
     GPIO.output(led_array[i], False)   
   # Infinite Loop   
   while (True):   
     for i in range(0, 8):   
       GPIO.output(led_array[i], True)   
       print led_array[i], 'pin On'   
       time.sleep(blink_delay)   
       GPIO.output(led_array[i], False)   
       print led_array[i], 'pin Off'   
       time.sleep(blink_delay)   
 except KeyboardInterrupt:   
   print "Exiting Program"   
 except:   
   print "Error Occurs, Exiting Program"   
 finally:   
   GPIO.cleanup()
