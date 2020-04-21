# daixijun.epel

[![Build Status](https://github.com/daixijun/ansible-role-epel/workflows/build/badge.svg)](https://github.com/daixijun/ansible-role-epel/actions)
[![Ansible Galaxy](https://img.shields.io/badge/galaxy-daixijun.epel-660198.svg?style=flat)](https://galaxy.ansible.com/daixijun/ansible-role-epel/)
[![GitHub tag (latest SemVer)](https://img.shields.io/github/v/tag/daixijun/ansible-role-epel?sort=semver)](https://github.com/daixijun/ansible-role-epel/tags)

为 RHEL/CentOS 系列系统安装配置 epel-release 仓库

## 环境要求

* RHEL/CentOS 6.x / 7.x / 8.x

## 变量

```yaml
# 是否需要替换 epel 的仓库
epel_repo_replace: false
# epel 仓库的 repo 文件地址
epel_repo_url: http://mirrors.aliyun.com/repo/epel-{{ ansible_distribution_major_version }}.repo
```

## 依赖

无

## 使用示例

```yaml
- hosts: servers
  roles:
    - { role: daixijun.epel }
```

## License

BSD

## 维护者

* Xijun Dai <daixijun1990@gmail.com>
