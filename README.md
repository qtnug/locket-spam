<b>Tool spam kêt bạn locket, python 3.11 (khác so với bản gốc dùng 3.7)</b>
Truy cập [Google colab](https://colab.google/) để chạy code
<details>
  <summary>Code (Python 3.11)</summary>

```python 3.11
import os

repo_path = "/content/locket-spam"
target_path = "/content"

if not os.path.exists(repo_path):
    !git clone https://github.com/qtnug/locket-spam.git {repo_path}

!mv {repo_path}/* {target_path}/
!mv {repo_path}/.* {target_path}/ 2>/dev/null
!rm -rf {repo_path}

!python3 app.py
```

</details>
