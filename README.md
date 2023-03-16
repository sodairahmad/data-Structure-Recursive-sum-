# data-Structure-Recursive-sum-


def sum(numbers):
    if not numbers:
        return 0 
    print(f" Calling sum {numbers[1:]}")
    recursive_sum = sum(numbers[1:])
    print(f"Call to sum {str(numbers)} returning {str(numbers[0])} + {recursive_sum}")
    return numbers[0] + recursive_sum

numbers = [1,2,3,9,99,33,88,103,835,847,9394,347]

print(sum(numbers))

