# DevCom-problemstatement2
this is the solution for the 2nd problem statement. 
I have created a function generateUpdateData to kinda help sync the devices and server, currently at times the code gets stuck in an infinite loop because it isn't able to sync some data point at certain times,v to counter that we can add a for loop to limit the maximum number of iterations. 
__init__(self): Initializes the synchronization service.
onMessage(self, data: dict) -> dict: Handles messages received from devices. It responds to probe requests with update data or acknowledges record messages. The method returns the appropriate response.
generateUpdateData(self, dev_id: str, from_index: int) -> dict: Generates update data based on the device ID and the requested index.
The testSyncing function simulates the interaction between multiple devices and the synchronization service. It creates instances of the Device and SyncService classes, generates data points, sends probe requests, and validates the synchronization process.

