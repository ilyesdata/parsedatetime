import parsedatetime.parsedatetime as pdt
import parsedatetime.parsedatetime\_consts as pdc

# create an instance of Constants class so we can override some of the defaults

c = pdc.Constants()

# create an instance of the Calendar class and pass in our Constants
# object instead of letting it create a default

p = pdt.Calendar(c)

# parse "tomorrow" and return the result

result = p.parse("tomorrow")

# parseDate() is a helper function that bypasses all of the
# natural language stuff and just tries to parse basic dates
# but using the locale information

result = p.parseDate("4/4/80")

# parseDateText() is a helper function that tries to parse
# long-form dates using the locale information

result = p.parseDateText("March 5th, 1980")