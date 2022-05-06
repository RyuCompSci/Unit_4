### produce a the average score of the students in the class

```.py
class Get_average:
    def __init__(self, students):
        self.students = students

    def avr(self):
        list_num = []
        sum = 0
        for item in self.students:
            list_num.append(item["score"])　# add the value to the list with hint
        for i in range(len(list_num)):
            sum += list_num[i]
        sum /= len(list_num) # gets the average
        sum = round(sum, 1) # round the value to 1 decimal place
        return sum
```

![](image_quiz_45.png)
