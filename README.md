// profile.cpp
constexpr struct Profile{
    auto name="Unrays"
        ,created="2025-09-25"
        ,location="Digital Realm";
    const char* skills[]{"C++","C#","Java", "JavaScript", "Dart", "SQL", "Python"};
    const char* tools[]{"VS Code","clang","Git","CMake","Docker"};
    constexpr auto motto(){ return "Talk is cheap, show me the code."; }
} profile{};
