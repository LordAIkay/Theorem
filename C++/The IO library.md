The IO library

- Header

  - ```C++
    #include <iostream>
    #include <fstream>
    #include <sstream>
    ```

- Condition state

  - goodbits, failbits, eofbits, badbits.

  - ```C++
    // use bit-wise operation to convey flagSSSSSS.
    void clear(strm::iostate flag = 0);// ???
    void setstate(strm::iostate flag);
    strm::iostate rdstate();
    ```

- File mode

  - in, out, trunc, app, ate, binary.

  - ```C++
    #include <fstream>
    //ifstream, ofstream, fstream.
    ofstream::ofstream(char* arg = nullptr, filemod fm = out);//trunc is implicit
    
    //default file modes are depends on fstream tyoe.
    void fstream::open(char* arg = nullptr, filemod fm = out/in);
    void fstream::close(char* arg = nullptr, filemod fm = out/in);
    bool fstream::is_open();
    ```

  - For ifstream, ofstream, fstream, different types have different default file mode.

  - `out` only for ofstream type, `in` only for ifstream type.

- `<sstream>`

  - ```C++
    #include <sstream>
    #include <string>
    //isstream, osstream, stringstream.
    using namespace std;
    sstream::sstream(string s); //explicit.
    string str();
    void str(sring s);
    ```



