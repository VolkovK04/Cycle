def take(seq, n):
    res = []
    for i in range(n):
        try:
            res.append(next(seq))
        except StopIteration:
            break
    return res


def cycle(iter):
    buff = iter.__iter__()
    while True:
        try:
            yield buff.__next__()
        except StopIteration:
            buff = iter.__iter__()
            yield buff.__next__()


if __name__ == '__main__':
    print(take(cycle([1, 2, 3]), 10))
