![image](https://github.com/Sadashiva84/TravelMemory/assets/137101252/703568a2-f0e9-484b-8f82-ef8ef9e4abd1)# Travel Memory
## This Project uses a cloud instance to be deployed

1. Backend Configuration:

   - Clone the repository and navigate to the backend directory.

   - The backend runs on port 3000. Set up a reverse proxy using nginx to ensure smooth deployment on EC2.

   - Update the .env file to incorporate database connection details and port information.

 2. Frontend and Backend Connection:

   - Navigate to the `urls.js` in the frontend directory.

   - Update the file to ensure the frontend communicates effectively with the backend.

 3. Scaling the Application:

   - Create multiple instances of both the frontend and backend servers.

   - Add these instances to a load balancer to ensure efficient distribution of incoming traffic.

 4. Domain Setup with Cloudflare:

   - Connect your custom domain to the application using Cloudflare.

   - Create a CNAME record pointing to the load balancer endpoint.

   - Set up an A record with the IP address of the EC2 instance hosting the frontend.





`.env` file to work with the backend:

```
MONGO_URI='ENTER_YOUR_URL'
PORT=3000
```

Data format to be added: 

```json
{
    "tripName": "Incredible India",
    "startDateOfJourney": "19-03-2022",
    "endDateOfJourney": "27-03-2022",
    "nameOfHotels":"Hotel Namaste, Backpackers Club",
    "placesVisited":"Delhi, Kolkata, Chennai, Mumbai",
    "totalCost": 800000,
    "tripType": "leisure",
    "experience": "Lorem Ipsum, Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum,Lorem Ipsum, ",
    "image": "https://t3.ftcdn.net/jpg/03/04/85/26/360_F_304852693_nSOn9KvUgafgvZ6wM0CNaULYUa7xXBkA.jpg",
    "shortDescription":"India is a wonderful country with rich culture and good people.",
    "featured": true
}
```
