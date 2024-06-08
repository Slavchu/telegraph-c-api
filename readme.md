# Telegraph API for C++
This is basic telegraph api that uses curl under its logic. For json used nlohmann json library.
## How to use it
There is only one class. To start work you have to create class TelegraphApi. Example:
```cpp
telegraph::TelegraphApi(telegraph::TelegraphApi::create_account("example shortname", "exmaple name", "example url"));
```
Function</br> TelegraphApi::uploadImage(std::string bin); </br>returns string with image url after upload image binary! 
```cpp
        std::string create_page(std::string title, std::vector<std::string> images, std::string text, std::string author_url = "", std::string author_name = "");

```
create_page method returns url for a page.</br>
## CMake
```CMake
add_subdirectory(Library relative directory path)
target_link_libraries(YourProject telegraph_api)


``` 
