# hw2.py
[Uploading practice.py…]()def exchange(amount):
    res_500 = int(amount // 500)
    amount %= 500

    res_100 = int(amount // 100)
    amount %= 100

    res_50 = int(amount // 50)
    amount %= 50

    res_10 = int(amount // 10)
    amount %= 10

print(f"500원 동전의 개수:res_500")
print(f"100원 동전의 개수: {res_100}")
print(f"50원 동전의 개수: {res_50}")
print(f"10원 동전의 개수: {res_10}")

def get_integer(prompt):
    value = int(input(prompt))
    if value < 0:
        print("0 이상의 금액만 입력해주세요.")
        return 0
    return value

def main():
    amount = get_integer("동전으로 교환하고자 하는 금액은? ")
    if amount > 0:
        exchange(amount)

if __name__ == "__main__":
    main()


