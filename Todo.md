A simple list of the "big" feature items we want to put into future versions.

The list is not ordered and not everything is guaranteed to make into the library.

## Parsing ##

  * Timezone support
  * Ability to scan large parts of text and extract any found date/time information

## API ##

  * Split out the parsing code and the date/time calculation code into their own modules
  * Get the parsing code to return a dictionary of items that have been flagged along with what their types are
  * Allow for chunks to "know" about their relation to other chunks and to have them weighted so calculated values can be influenced.  For example: "Aug 22 at 11am" would have the "Aug 22" part know it's right next to the "11am" part and since one is a date and the other a time and the seperation is a task/event oriented word..... :)
  * Allow for a flag to have the API only return the values that are known and not fill in from the current or source date/time.