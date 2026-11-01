# Amoral Client runtime

Готовые сборки [Jep](https://github.com/ninia/jep) — моста Python ↔ Java, на котором работают
Python-скрипты Amoral Client. Клиент сам скачивает нужный файл из релиза
[`python-runtime`](../../releases/tag/python-runtime) при первом запуске скриптов, поэтому игрокам не
нужны ни компилятор C, ни Microsoft C++ Build Tools.

| Файл | Платформа |
|---|---|
| `jep-4.2.2-x86_64-pc-windows-msvc.whl` | Windows x64 |
| `jep-4.2.2-x86_64-unknown-linux-gnu.whl` | Linux x64 |
| `jep-4.2.2-aarch64-unknown-linux-gnu.whl` | Linux ARM64 |
| `jep-4.2.2-aarch64-apple-darwin.whl` | macOS Apple Silicon |
| `jep-4.2.2-x86_64-apple-darwin.whl` | macOS Intel |

Файлы — zip-архивы содержимого `site-packages` после `pip install --target` под Python 3.10;
клиент распаковывает их во встроенный Python (python-build-standalone 3.10).

Сборка: [.github/workflows/build.yml](.github/workflows/build.yml) (Actions → Run workflow).

Jep распространяется по лицензии zlib/libpng, см. [LICENSE-jep](LICENSE-jep).
