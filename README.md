<b>Tool spam kêt bạn locket, python 3.11 (khác so với bản gốc dùng 3.7)</b>
<p>Nhiều proxy hơn bản gốc. Tools gốc có tầm 11.000 proxy. Mình đã cập nhật list proxy lên tận <b>100.000</b> proxy</p>
<p>Truy cập [Google colab](https://colab.google/) để chạy code</p>
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
