### Ascii art

```.py
class Ascii():
    def __init__(self, input):
        self.input = input.lower()
        self.alphabet = [
         "### ##   ## ##  ### ###  ## # # ###  ## # # #   # # ###  #  ##   #  ##   ## ### # # # # # # # # # # ### ###",
         "# # # # #   # # #   #   #   # #  #    # # # #   ### # # # # # # # # # # #    #  # # # # # # # # # #   #   # ",
         "### ##  #   # # ##  ##  # # ###  #    # ##  #   ### # # # # ##  # # ##   #   #  # # # # ###  #   #   #   ## ",
         "# # # # #   # # #   #   # # # #  #  # # # # #   # # # # # # #    ## # #   #  #  # # # # ### # #  #  #       ",
         "# # ##   ## ##  ### #    ## # # ###  #  # # ### # # # #  #  #     # # # ##   #  ###  #  # # # #  #  ###  #  "
        ]
        self.result = ""

    def convert(self):
        for j in self.alphabet: # for each line that builds each character
            for i in self.input:
                ascii = ord(i) - 97 # convert letters in input into ascii notation
                character = [4*ascii, 4+4*ascii] # get the range of each character
                self.result += j[character[0]:character[1]] # take a line for all letters
            self.result += "\n"
        return self.result
```

![]()
