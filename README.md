# DSA-Essentials-Bootcamp2
Assignment - DSA Essentials Bootcamp

def find_duplicates(nums):
    duplicates = []
    count = {}

    for num in nums:
        if num in count:
            count[num] += 1
        else:
            count[num] = 1

    for num, freq in count.items():
        if freq == 2:
            duplicates.append(num)

    return duplicates

    
nums = [4, 3, 2, 7, 8, 2, 3, 1]
result = find_duplicates(nums)
print(result)
