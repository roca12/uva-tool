# uva-tool
Command Line Based Tool for [uva onlinejudge](https://uva.onlinejudge.org/) with feature Submitting and uHunting.

## Dependency
- Command line based tool [`curl`](https://curl.haxx.se/)
- [`nlohmann json`](https://github.com/nlohmann/json) C++ library

## Installation
- **Install `curl`:** Download and install [curl](https://github.com/curl/curl) (website: https://curl.haxx.se/). On ubuntu to install curl execute  
`sudo apt install curl`.
- **Download uva-tool:** Execute command `git clone https://github.com/AHJenin/uva-tool.git`.
- **Install uva-tool:** In the downloaded folder `uva-tool`, look for `install.sh` file and execute it (C++ compiler needed here, GNU g++ used in testing).  
`chmod +x install.sh`  
`sudo ./install.sh`


## Usage Example
Run corresponding commands
- **Login:** `uva-tool -login`
- **Logout:** `uva-tool -logout`
- **Hunt:** `uva-tool -hunt -u felix_halim -r 10`  
This will show last 10 submission of user `felix_halim`
- **Submit:** Sysntax `uva-tool -submit problem_number problem_path language`, example `uva-tool -submit 100 ~/Desktop/100.cpp 5`. This will submit `100.cpp` named file from Desktop directory in C++11 (5 for C++11) language with problem number 100. Language codes  
1 = ANSI  
2 = JAVA  
3 = C++  
4 = Pascal  
5 = C++11  
6 = Python


