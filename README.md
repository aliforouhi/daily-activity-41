# daily_update.p
import datetime
import random

print("Daily GitHub activity - Day 41")

today = datetime.date.today()

# Generate random website response times (ms) and analyze
response_times = [random.randint(80, 450) for _ in range(8)]
slow_requests = [t for t in response_times if t > 300]

print(f"Today's date: {today}")
print("Response times (ms):", response_times)
print("Fastest response:", min(response_times), "ms")
print("Slowest response:", max(response_times), "ms")
print("Slow requests (>300 ms):", len(slow_requests))
