# pythonexamples
```
abs(-34.5)
math.ceil(2.15), math.floor(3.14), math.sqrt(225), math.isclose()

min(x, -4)
max(3.14, y)
pow(2.71, 3.14) or 2.71 ** 3.14
str(42), str(3.144)
int('42')
float('3.14'), float('inf'), float('-inf')
```

```
random.randrange(5), random.randint(8, 16), random.random(), random.shuffle(A), random.choice(A)
```

```
raise ValueError('All bits are 0 or 1')
```

```
list(range(100))
[0] * 10
len(A), A.append(20), A.insert(4, 50), A.remove(50), del A[4]
B = list(A), copy.copy(A), copy.deepcopy(A)
```

```
bisect.bisect(A, x), bisect.bisect_left(A, x), bisect.bisect_right(A, 6)
```

```
A[::-1], B = A[:], A[k:] + A[:k]
[x**2 for x in range(6) if x % 2 == 0]
[[x**2 for x in row] for row in A]
```

```
A[equal], A[larger] = A[larger], A[equal]
```

```
gen_o_nums = (x for x in range(100))
result[next(
            (i for i, x in enumerate(result) if x != 0),
            len(result)
            ):] or [0]

return [sign * result[0]] + result[1:]
```

```
initial_array = [0.0] * len(stocks)
```

```
for i in range(5):
for i, element in enumerate(a_list):
```

```
sorted(a_list, reverse=bool(i % 2))
```

```
perm[inversionPoint + 1:] = reversed(perm[inversionPoint + 1:])
```

```
itertools.islice(stream_iterator, k)
prefix_sum_probabilities = list(itertools.accumulate(probabilities))
```

```
index = bisect.bisect(prefix_sum_probabilities, random.random())
```

```
new_list = filter(lambda x: x != 0, old_list)
```

```
for c in s:
```

```
s.strip(), s.startswith(prefix), s.endswith(suffix), 'sample, string'.split(','), s.tolower(), s.isalnum()
','.join(list_string), ','.join(('A', 'B', 'C'))
string.hexdigits[value]
```

```
new_char = chr(ord('0') + 5)
```

```
functools.reduce(lambda acc, ele: acc + ele, input_list, initial_value)
```

```
with open(file_path, 'r') as open_file:
    text = open_file.readlines()
    policy = json.load(open_file)
    verify_apache = yaml.safe_load(open_file)
    off_reader = csv.reader(csv_file, delimiter=',')
        for _ in range(5):
            print(next(off_reader))

with open('.envrc', 'w') as opened_file:
    opened_file.write(text)
    policy = json.dump(policy, opened_file)
    yaml.dump(verify_apache, opened_file)

path = pathlib.Path("/Users/kbehrman/projects/autoscaler/check_pending.py")
path.read_text()
path.write_text("LOG:DEBUG")
```

```
# Generator for reading big files
def big_file_line_reader(file_path):
    with open(file_path, 'r') as source_file:
        for line in source_file:
            yield line
reader = big_file_line_reader('file')
for line in reader:
    process(line)
```

```
subprocess.run(['ls', '-l'], capture_output=True, universal_newlines=True, check=True)
subprocess.run(['ls', '-l'], capture_output=True, universal_newlines=True, check=True, shell=True)
```

```
./sys_argv.py --a-flag    some-value   13
sys.argv[0]   sys.argv[1] sys.argv[2]  sys.argv[3]
```

```
argparse, click
```

```
import requests, logging
logger = logging.getLogger()
sess = requests.session()
sess.get(), sess.post()
```

```
# disable self signed certificate warnings
requests.packages.urllib3.disable_warnings()
sess.post(..., verify=False)
# in some cases, authentication cookie will be retained in the session. No need to send token
```

```
https://github.com/nickrusso42518/slt-py-requests
```

```
# set a breakpoint for debugging
breakpoint() # py 3.7+
import pdb; pdb.set_trace() # py 3.6-
```
