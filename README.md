# Encryption Proxy Gateway

Functionality: Transfer files that are end-to-end encrypted between an origin server and a frontend client

This Gateway looks like this:
![product](/images/image-3.png)

### Architecture Diagram
A diagram of the architecture and choose the stack:

- Diagram the architecture and agree on stack
- Implement:
  - API: Frontend ←→ Server M
  - API: Server M ←→ Server E

![architecture-diagram](/images/image-5.png)

### Run Locally
In order to run the code locally, we need to have three terminals to run frontend, server-e, and server-m seperately.
```bash
Run Frontend:
1. open the terminal
2. cd frontend
3. npm install
4. npm start

when you see "Compiled successfully!", that means it runs successfully
```

```bash
Run server-e and server-m:
1. open the second terminal
2. cd servers3. 
3. npm install
4. node server-e.js

when you see "Server E listening at http://localhost:80", that means it runs successfully

5. switch to the third terminal
6. cd servers
7. node server-m.js

when you see "Server M listening at http://localhost:3000", that means it runs successfully
```

After those steps, please try on frontend, and upload file, you can get both Encrypted File and Decrypted File by clicking on corresponding buttons 

### Run Tests

```bash
1. open tests
2. open a terminal
3. npm install --save-dev @testing-library/react @testing-library/jest-dom jest @types/jest
4. npx jest serverME.test.js
```
