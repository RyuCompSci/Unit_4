### Sort an array from the smallest to the largest

```.py
class List_sort:
    def __init__(self, lst:list):
        self.lst = lst

    def sort(self):
        sorted_lst = [] # list for the output
        length = len(self.lst)
        for j in range(len(self.lst)-1):
            smallest = self.lst[0] # define that the first value of the list is smallest
            for i in range(length-1):
                if self.lst[i+1] <= smallest:
                    smallest = self.lst[i+1]
            sorted_lst.append(smallest) # adds the new smallest number to the sorted_lst
            self.lst.remove(smallest) # extracts the smallest number from the lst
            length -= 1
        return sorted_lst
```

![]()
