def convert_to_binary(number):
    if number == 0:
        return "0"

    result = ""

    while number > 0:
        result = str(number % 2) + result
        number //= 2

    return result


if __name__ == "__main__":
    number = 42

    print("Number:", number)
    print("Binary:", convert_to_binary(number))
