# ansible-role-textual

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-textual.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-textual)

macOS - Textual IRC Client

## Requirements

This role requires Homebrew and Homebrew Cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    textual_pkg: Textual
    textual_domain: "com.codeux.apps.{{ textual_pkg|lower }}"
    textual_defaults: {}

## Dependencies

  * https://galaxy.ansible.com/geerlingguy/homebrew

## Example Playbook

    - hosts: localhost
      connection: local
      roles:
        - role: tkimball83.textual
          textual_defaults:
            CopyTextSelectionOnMouseUp:
              type: int
              value: 1
            InvertSidebarColors:
              type: int
              value: 1
            MemberListSortFavorsServerStaff:
              type: int
              value: 1
            NicknameColorHashingComputesRGBValue:
              type: int
              value: 1
            RejoinChannelOnLocalKick:
              type: int
              value: 1
            ReplyUnignoredExternalCTCPRequests:
              type: int
              value: 0
            SUAutomaticallyUpdate:
              type: int
              value: 1
            SUEnableAutomaticChecks:
              type: int
              value: 1
            ServerListDoubleClickConnectServer:
              type: int
              value: 1
            ServerListDoubleClickDisconnectServer:
              type: int
              value: 1
            ServerListDoubleClickJoinChannel:
              type: int
              value: 1
            ServerListDoubleClickLeaveChannel:
              type: int
              value: 1
            TextFieldAutomaticGrammarCheck:
              type: int
              value: 0
            TextFieldAutomaticSpellCheck:
              type: int
              value: 0

## License

GPLv3

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
