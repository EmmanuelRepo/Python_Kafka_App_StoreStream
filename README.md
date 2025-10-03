Python_Kafka_App_StoreStream/
├── producer.py           # Python Kafka Producer
├── tacker.py             # Python Kafka Consumer/Tracker
├── docker-compose.yaml   # Docker Compose for Kafka & Zookeeper
└── .idea/                # IDE settings (can be ignored or added to .gitignore)

🚀 Getting Started
Prerequisites

Python 3.8+

Docker & Docker Compose

pip (Python package manager)

git clone https://github.com/EmmanuelRepo/Python_Kafka_App_StoreStream.git
cd Python_Kafka_App_StoreStream

docker-compose up -d


This will start:

Zookeeper

Kafka broker (on port 9092)


3. Install Python Dependencies

Create and activate a virtual environment (optional but recommended):

python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Then install required libraries:

pip install kafka-python

4. Run the Producer and Consumer
Start the Kafka Consumer (Tracker):
python tacker.py

Start the Kafka Producer:
python producer.py


You should see messages being produced and consumed via the terminal.

🧪 Example Output
[Producer] Sent: {"event": "new_user", "user_id": 123}
[Consumer] Received: {"event": "new_user", "user_id": 123}

🛠️ Future Improvements

Add logging instead of print statements

Add unit tests and Dockerized test suite

Expand to multiple topics or more complex message schemas

Integrate with Kafka Streams or Kafka Connect

📝 License

MIT License. Feel free to use, modify, and share.

🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss your ideas.
