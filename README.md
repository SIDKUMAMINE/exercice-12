# exercice-12

def ordinalDate(day, month, year):
    is_leap_year = (year % 4 == 0 and year % 100 != 0) or (year % 400 == 0)
    days_in_month = [31, 28 + is_leap_year, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
    day_of_year = sum(days_in_month[:month-1]) + day
    return day_of_year
