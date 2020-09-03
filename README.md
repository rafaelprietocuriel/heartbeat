# heartbeat
Compute weekly heartbeats of data on R and RStudio

Function to compute the heartbeat of some data
Author: Rafael Prieto Curiel rafael.prieto.13@ucl.ac.uk
Input: Time of the events, provided as a single number
       where the number 43831.0 represents Wednesday 01/01/2020
       the integer part represents the day and the decimal part
       of the number represents the time of the day, so that
       43831.50 is Wednesday 01/01/2020 at 12:00
       43831.25 is Wednesday 01/01/2020 at 6:00, and
       43831.75 is Wednesday 01/01/2020 at 18:00

Output: The heartbeat of the events, smoothed with a cyclic KDE
        computed for a vector of length 1024. 
        The first entry corresponds to Monday at 0:00
        The entry 100 corresponds to Monday at 16:24, and
        The entry 147 corresponds to Tuesday at 0:07 
