class SampleClass:
  def __init__(self, value):
    self.__value = value
  def __method(self):
    print(self.__value)


sample_instance = SampleClass("Hello!")
vars(sample_instance)

