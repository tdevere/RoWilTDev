# NOTES

## 11/9

### Create a list of strings with data

    Review Line 27 of the script. This is just another way to do the same thing in one step. 

    $myArray = @("Hello", "World", "from", "PowerShell")

### Get Start and End Date of current month

    # Get the current date
    $today = Get-Date

    # Get the last day of the current month
    $lastDay = [DateTime]::DaysInMonth($today.Year, $today.Month)

    # Create DateTime objects for the first and last day of the month
    $firstDate = [DateTime]::new($today.Year, $today.Month, 1)
    $lastDate = [DateTime]::new($today.Year, $today.Month, $lastDay)

    # Display the first and last dates of the month
    $firstDate
    $lastDate
