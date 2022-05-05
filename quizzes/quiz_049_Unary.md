### Unary

```.py
class Unary:
    def __init__(self, binary:int):
        self.binary = str(binary)

    def convert_to_unary(self):
        unary = ""
        zeros = ""
        num = "0"
        n = 0
        nn = 0
        for i in range(len(self.binary)-1):
            if self.binary[i] == self.binary[i+1]:
                num += "0"
            else:
                zo = self.binary[i]
                if zo == "0":
                    zeros = "00"
                elif zo == "1":
                    zeros = "0"
                unary = unary + zeros + " " + num + " "
                num = "0"
        zo = self.binary[i]
        if zo == "0":
            zeros = "00"
        elif zo == "1":
            zeros = "0"
        unary = unary + zeros + " " + num + " "
        return unary
```

![]()
