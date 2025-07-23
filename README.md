import datetime
import time

class Timer(object):
    """A simple timer class"""
    def start(self):
        self.start_time = datetime.datetime.now()
        print("Stopwatch started.")
    def stop(self):
        self.end_time = datetime.datetime.now()
        print("Stopwatch stopped.")
        print("Elapsed:", self.end_time - self.start_time)

timer = Timer()
timer.start()
input("Press Enter to stop the stopwatch...")
timer.stop()
