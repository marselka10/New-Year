# New-Year
from datetime import datetime

def days_until_new_year():
    today = datetime.now()
    new_year = datetime(today.year + 1, 1, 1)
    if today.month == 12 and today.day == 31:
        return 0  # if today is already December 31st
    days_remaining = (new_year - today).days
    return days_remaining

print(f"Number of days until New Year 2025: {days_until_new_year()}")
