# People You May Know (Friend Recommendation Engine)

This repository contains a Python-based recommendation algorithm that mimics the "People You May Know" feature found on modern social media platforms. It analyzes a network dataset to suggest new friends based on the frequency of mutual connections.

## Features
* **Network Analysis:** Maps out users and their direct connections using Python sets for optimized $O(1)$ lookups.
* **Intelligent Filtering:** Automatically removes the target user and their existing direct friends from the pool of potential suggestions.
* **Ranked Output:** Calculates the number of mutual friends for each "friend of a friend" and sorts the final recommendations in descending order, ensuring the most relevant people are suggested first.

## Prerequisites
To run this project, you need:
* **Python 3.x** installed on your system.
* A JSON file (e.g., `massivedata.json`) containing the network data. The expected structure is a list of users, where each user has an `"id"` and a list of `"friends"`.

## Usage

1. Clone this repository or download the files directly to your computer.
2. Ensure your dataset (`massivedata.json`) is in the same directory as the Python script.
3. Run the script using Python:
   ```bash
