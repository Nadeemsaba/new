class SampleClass:
    def __init__(self, value):
        self.__value = value  # private variable

    def __method(self):
        print(self.__value)  # private method accessing private variable

    def public_method(self):
        # Access private method from a public interface
        self.__method()


sample_instance = SampleClass("Hello!")
sample_instance.public_method()

# To see mangled variable name
print(vars(sample_instance))  # Output will have '_SampleClass__value'
