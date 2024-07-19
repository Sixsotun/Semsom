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

function switchTheme() {
  wrapper.classList.toggle('dark-theme')
  wrapper.classList.toggle('light-theme')

  if (wrapper.classList.contains('dark-theme')) {
    localStorage.setItem('theme', 'dark')
  } else {
    localStorage.setItem('theme', 'light')
  }
}

if (localStorage.getItem('theme') == 'dark') {
  themeSwitcher.setAttribute('checked', '')
  switchTheme()
} else {
  themeSwitcher.removeAttribute('checked')
}

themeSwitcher.addEventListener('click', switchTheme)
