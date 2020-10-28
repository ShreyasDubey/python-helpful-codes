# python-helpful-codes
#all small techniques to take refrence later
# code to find if nos are absolute increasing
import ast,sys
input_str = sys.stdin.read()
input_list = ast.literal_eval(input_str)

if all(i < j for i, j in zip(input_list, input_list[1:])):
    print("yes")
else:
    print("no")
