# CivKit CLI Functionalities

This document outlines the functionalities of the CivKit CLI, detailing the user actions and the corresponding backend processes for each command.

## Functionalities

### **ping** (Send a ping message)
- **User Action**: A button labeled "Ping" that, when clicked, sends a ping request.
- **Backend Process**: The backend receives the ping request and responds, possibly with a pong message or a status update.

### **shutdown** (Shutdown the connected CivKit node)
- **User Action**: A "Shutdown" button that, when clicked, initiates the shutdown process.
- **Backend Process**: The backend safely shuts down the connected CivKit node.

### **publishtextnote** (Send a demo NIP-01 EVENT kind 1)
- **User Action**: A text input field and a submit button for users to send a text note.
- **Backend Process**: The backend publishes the text note to all connected clients.

### **listclients** (List information about connected clients)
- **User Action**: A "List Clients" button that displays the connected clients.
- **Backend Process**: The backend retrieves and sends a list of all connected clients.

### **listsubscriptions** (List information about subscriptions)
- **User Action**: A button or section in the UI to view current subscriptions.
- **Backend Process**: The backend provides a list of current subscriptions.

### **connectpeer** (Connect to a BOLT8 peer)
- **User Action**: An interface for entering peer details and a button to initiate connection.
- **Backend Process**: The backend attempts to connect to the specified BOLT8 peer.

### **disconnectclient** (Disconnect from a client)
- **User Action**: Options in the client list to disconnect from a specific client.
- **Backend Process**: The backend disconnects from the selected client.

### **publishnotice** (Send a demo NIP-01 NOTICE)
- **User Action**: A form to create and send a notice.
- **Backend Process**: The backend publishes the notice to all connected clients.

### **publishoffer** (Send BOLT12 offers)
- **User Action**: A UI for creating and sending BOLT12 offers.
- **Backend Process**: The backend sends the created offers to all connected clients.

### **publishinvoice**
- **User Action**: A feature to create and publish invoices.
- **Backend Process**: The backend handles the publishing of the invoice.

### **list-db-events** (List DB entries)
- **User Action**: A "List Database Events" button or section.
- **Backend Process**: The backend retrieves and displays database event entries.

### **list-db-clients** (List DB clients entries)
- **User Action**: A feature to view a list of database clients.
- **Backend Process**: The backend provides a list of clients from the database.

### **check-chain-state** (Check chain state)
- **User Action**: A button or feature to check the current state of the chain.
- **Backend Process**: The backend checks and returns the current state of the chain.

### **generate-tx-inclusion-proof** (Generate a merkle block for the target txid)
- **User Action**: An interface for inputting a transaction ID and requesting its inclusion proof.
- **Backend Process**: The backend generates and returns the merkle block for the given transaction ID.

### **help** (Print help message)
- **User Action**: A "Help" button or section in the UI.
- **Backend Process**: The backend provides help information or documentation for the commands.
