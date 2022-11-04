## NodeJS

## Normalization directory path
<pre>
function normalize_directory_path(input) {
    let arr = input.split('/')

    let skip_parent = 0;
    let output = ""
    for (let i = arr.length - 1; i > 0; i--) {
        if (arr[i] == "." || arr[i] == "") {
            continue;
        }
        if (arr[i] == "..") {
            skip_parent += 1
        } else {
            if (skip_parent > 0) {
                skip_parent -= 1
            } else {
                if (output) {
                    output = arr[i] + "/" + output
                } else {
                    output = arr[i]
                }
            }
        }
    }
    if (!output) {
        console.log('/')
    } else {
        console.log("/" + output)
    }
}

normalize_directory_path("/etc/system/../../home/user")
normalize_directory_path("/home/../..")
normalize_directory_path("/usr/local/./../bin/.")
normalize_directory_path("/a/./b")
normalize_directory_path("/a/../b")
normalize_directory_path("/a/.../b")
normalize_directory_path("/a////b")
normalize_directory_path("/../a")
normalize_directory_path("/usr/./././../a")
</pre>