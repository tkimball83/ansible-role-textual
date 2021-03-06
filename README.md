# ansible-role-textual

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-textual.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-textual)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-textual-blue.svg?style=flat)](https://galaxy.ansible.com/tkimball83/textual)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](COPYING)

macOS - Textual IRC Client

## Requirements

This role requires homebrew and homebrew cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    textual_defaults: []
    textual_domain: "com.codeux.apps.{{ textual_package|lower }}"
    textual_package: Textual

## Dependencies

None

## Example Playbook

    - hosts: localhost
      connection: local
      roles:
        - role: tkimball83.textual
          textual_defaults:
            - name: CopyTextSelectionOnMouseUp
              type: bool
              value: true
            - name: InvertSidebarColors
              type: bool
              value: true
            - name: MemberListSortFavorsServerStaff
              type: bool
              value: true
            - name: NicknameColorHashingComputesRGBValue
              type: bool
              value: true
            - name: RejoinChannelOnLocalKick
              type: bool
              value: true
            - name: ReplyUnignoredExternalCTCPRequests
              type: int
              value: 0
            - name: SUAutomaticallyUpdate
              type: bool
              value: true
            - name: SUEnableAutomaticChecks
              type: bool
              value: true
            - name: ServerListDoubleClickConnectServer
              type: bool
              value: true
            - name: ServerListDoubleClickDisconnectServer
              type: bool
              value: true
            - name: ServerListDoubleClickJoinChannel
              type: bool
              value: true
            - name: ServerListDoubleClickLeaveChannel
              type: bool
              value: true
            - name: TextFieldAutomaticGrammarCheck
              type: bool
              value: false
            - name: TextFieldAutomaticSpellCheck
              type: bool
              value: false

## License

Copyright (C) 2018 Taylor Kimball <tkimball@linuxhq.org>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
