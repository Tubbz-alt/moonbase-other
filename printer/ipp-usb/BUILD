export GOFLAGS="-buildmode=pie -trimpath -mod=readonly -modcacherw" &&

make &&

prepare_install &&

mkdir -p /etc/ipp-usb

install -Dm755 $MODULE /usr/bin/ &&
install -Dm644 ipp-usb.conf /etc/ipp-usb/ &&
install -Dm644 systemd-udev/71-ipp-usb.rules /usr/lib/udev/rules.d/ &&
install -Dm644 systemd-udev/ipp-usb.service /usr/lib/systemd/system/ &&
install -Dm644 ipp-usb.8 /usr/share/man/man8/ &&
install -Dm644 ipp-usb-quirks/* -t /usr//share/ipp-usb/quirks
