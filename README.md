This is a fork from https://github.com/LibrePDF/OpenPDF


# Prerequisites

1. Java 11
1. Maven 3.6.3

    1. On macOS, `brew install https://raw.githubusercontent.com/Homebrew/homebrew-core/ae5d1817d06d6350f4a8d657a01e4b8bd9bee61c/Formula/maven.rb`
        1. This avoid installing the dependency openjdk-14
            1. brew team refuses to not install its own openjdk https://github.com/Homebrew/homebrew-core/pull/51887
        1. This commit is taken from https://github.com/Homebrew/homebrew-core/pull/47242
            1. Since the github history fails to generate (taking too long) https://github.com/Homebrew/homebrew-core/commits/master/Formula/maven.rb
        1. `brew install --ignore-dependencies maven` results in

                Error: An exception occurred within a child process:
                  RuntimeError: /usr/local/opt/openjdk not present or broken
                Please reinstall openjdk. Sorry :(


# Run the tests

        cd openpdf
        mvn test
