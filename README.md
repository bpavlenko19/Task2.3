# Task2.3
from flask import Flask, request, jsonify

app = Flask(__name__)

@app.route('/subscribe', methods=['POST'])
def subscribe_user():
    # Реалізація підписки користувача
    return jsonify({'message': 'Subscription successful'}), 201

if __name__ == '__main__':
    app.run(port=5003)
