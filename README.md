# automatic_parking_sys_using_binary_semaphore
this project is based on the concept of semaphores and scheduling used for automated parking.
The vehicles enter the parking system in two queues. Only one vehicle can enter the parking system/machine at a time.
 
P and V Semaphores are used to avoid deadlock whenever a vehicle enter into machine function P is called which decrements the value of S (constant) to 0 and until S equal’s one no other vehicle can enter the machine and when vehicle get parked it calls function V which increments S to 1 so now other vehicle can also enter the machine.
 
We have done this for two-wheelers and four-wheeler’s separately. Then the vehicles reach the automatic parking machines and are left in the machine to start the process of automatic parking. The machine automatically parks the vehicles. This can be explained as : The parking machine is a critical section and the vehicles are processes. 

The parking entrance of 2 rows acts as a lock Only one process can enter the critical section/shared memory at a time in each row one four-wheeler and one two-wheeler. 
The processes(here vehicles) are then parked(scheduled) on the basis of first come first serve and semaphore. The processes the leave the shared memory and next vehicle can enter the parking area.
