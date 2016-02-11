FROM fabric8/swift:2.2-SNAPSHOT

ONBUILD RUN mkdir -p /usr/src/app
ONBUILD COPY Package.swift /usr/src/app/
ONBUILD COPY Sources /usr/src/app/
ONBUILD RUN swift build --chdir /usr/src/app

CMD /usr/src/app/.build/debug/app
