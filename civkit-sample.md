# CivKit Application Functionalities

This document outlines the key functionalities of the CivKit application, detailing both the user actions and the corresponding backend processes.

## Functionalities

### **sendtextnote** (Send a text note to the relay)
- **User Action**: Users can input a text message in a text field and submit it.
- **Backend Process**: The message is sent to a specified relay in the backend.

### **setmetadata** (Set the client's metadata)
- **User Action**: Users fill out a form with metadata details, which could include settings or preferences.
- **Backend Process**: The submitted metadata is used to update the client's profile or settings in the backend.

### **recommendserver** (Recommend a server to the relay)
- **User Action**: Users select or input a server recommendation, possibly from a list or a text input.
- **Backend Process**: The recommendation is sent to the relay for processing or storage.

### **sendmarketorder** (Send a market order to the relay)
- **User Action**: Users complete a form to create a market order, specifying details like order type, quantity, price, etc.
- **Backend Process**: The market order is processed and sent to the appropriate market or exchange relay.

### **opensubscription** (Open a subscription to the relay)
- **User Action**: Users choose to subscribe to a service or feed, possibly through a toggle or button.
- **Backend Process**: A subscription is initiated in the backend, enabling the user to receive updates or data feeds.

### **closesubscription** (Close a subscription to the relay)
- **User Action**: Users can opt to end a subscription, likely through a similar interface used to open it.
- **Backend Process**: The user’s subscription is terminated in the backend.

### **submitcredentialproof** (Submit a credential proof to the relay)
- **User Action**: Users might need to upload or enter credential information for verification purposes.
- **Backend Process**: The provided credentials are verified and authenticated by the backend.

### **addservice** (Register manually a service)
- **User Action**: Users input details of a new service they wish to register, typically through a detailed form.
- **Backend Process**: The service details are processed and the service is registered in the backend system.

### **shutdown** (Shutdown the REPL)
- **User Action**: This could be a simple button to safely shut down a session or service.
- **Backend Process**: The backend processes the shutdown command, terminating the session or service safely.

### **verifyinclusionproof** (Verify inclusion proof)
- **User Action**: Users might need to input or upload data for inclusion proof verification.
- **Backend Process**: The backend verifies the inclusion proof against stored data or a blockchain.

### **help**
- **User Action**: Users can request help or instructions, likely through a help button or command.
- **Backend Process**: The backend provides the relevant help information or documentation.
