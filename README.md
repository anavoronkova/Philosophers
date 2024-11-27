# Philosophers

### I Never Thought Philosophy Would Be So Deadly

#### Summary
**Philosophers** is a project that simulates the classic dining philosophers problem using threading and mutexes in C. The goal is to learn the basics of threading, mutexes, and synchronization to prevent race conditions and ensure the philosophers do not starve.

#### Introduction
The **Philosophers** project is a simulation where multiple philosophers sit at a table with a bowl of spaghetti. Philosophers alternate between eating, thinking, and sleeping, using forks that are shared among them. The simulation aims to manage these actions using threads and mutexes to avoid issues like deadlock or starvation.

#### Installation
1. Clone the repository:
   ```
   git clone <repository_url>
   ```
2. Navigate to the project directory:
   ```
   cd philosophers
   ```
3. Compile the project:
   ```
   make
   ```

#### Usage
Run the program with:
```
./philo <number_of_philosophers> <time_to_die> <time_to_eat> <time_to_sleep> [number_of_times_each_philosopher_must_eat]
```
- `<number_of_philosophers>`: Number of philosophers and forks.
- `<time_to_die>`: Time in milliseconds before a philosopher dies without eating.
- `<time_to_eat>`: Time in milliseconds it takes for a philosopher to eat.
- `<time_to_sleep>`: Time in milliseconds a philosopher spends sleeping.
- `[number_of_times_each_philosopher_must_eat]` (optional): Number of times each philosopher must eat before the simulation ends.

#### Features
- **Threading and Mutexes**: Each philosopher is a thread, and forks are protected by mutexes to prevent race conditions.
- **Synchronization**: Ensures that no two philosophers use the same fork simultaneously.
- **Real-Time Logs**: Logs the state changes of philosophers (eating, sleeping, thinking) with timestamps.
- **Bonus**: Includes an alternate implementation using processes and semaphores.

