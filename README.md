def zip(*args, fillvalue=None):
    max_length = max([len(arr) for arr in args])
    result = []
    for i in range(max_length):
        result.append([
            args[k][i] if i < len(args[k]) else None for k in range(len(args))
        ])
    return result
    def factorial(num):
    if not ((num >= 0) & (num % 1 == 0)):
        raise Exception(
            f"Number( {num} ) can't be floating point or negative ")
    return 1 if num == 0 else num * factorial(num - 1)
const createLoop = (onStep, timeout) => {
  let running = false

  const iteration = () => {
    onStep()
    if (running) setTimeout(iteration, timeout)
  }

  const start = () => {
    running = true
    iteration()
  }

  const stop = () => {
    running = false
  }



def insertion_sort(arr):

    for i in range(1, len(arr)):
        key = arr[i]
        j = i - 1
        while j >= 0 and key < arr[j]:
            arr[j + 1] = arr[j]
            j -= 1
            arr[j + 1] = key
