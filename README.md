#!/data/data/com.termux/files/usr/bin/bash

echo "===== Termux Setup Script ====="
echo "Updating package list..."
pkg update -y && pkg upgrade -y

echo "Installing basic packages: git, curl, wget, nano, python, neofetch"
pkg install -y git curl wget nano python neofetch

echo "Membuat folder kerja di ~/project"
mkdir -p ~/project

echo "Menampilkan informasi sistem dengan neofetch:"
neofetch

echo "Semua selesai! Silakan cek folder ~/project dan tools yang sudah terpasang."
