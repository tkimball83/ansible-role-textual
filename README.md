# ansible-role-textual

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-textual.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-textual)

macOS - Textual IRC Client

## Requirements

This role requires homebrew and homebrew cask to be installed

## Role Variables

Available variables are listed below, along with default values:

    textual_pkg: Textual
    textual_domain: "com.codeux.apps.{{ textual_pkg|lower }}"
    textual_defaults: {}

## Dependencies

None

## Example Playbook

    - hosts: localhost
      connection: local
      roles:
        - role: tkimball83.textual
          textual_defaults:
            CopyTextSelectionOnMouseUp:
              type: bool
              value: true
            InvertSidebarColors:
              type: bool
              value: true
            MemberListSortFavorsServerStaff:
              type: bool
              value: true
            NicknameColorHashingComputesRGBValue:
              type: bool
              value: true
            RejoinChannelOnLocalKick:
              type: bool
              value: true
            ReplyUnignoredExternalCTCPRequests:
              type: int
              value: 0
            SUAutomaticallyUpdate:
              type: bool
              value: true
            SUEnableAutomaticChecks:
              type: bool
              value: true
            ServerListDoubleClickConnectServer:
              type: bool
              value: true
            ServerListDoubleClickDisconnectServer:
              type: bool
              value: true
            ServerListDoubleClickJoinChannel:
              type: bool
              value: true
            ServerListDoubleClickLeaveChannel:
              type: bool
              value: true
            TextFieldAutomaticGrammarCheck:
              type: bool
              value: false
            TextFieldAutomaticSpellCheck:
              type: bool
              value: false

## License

GPLv3

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
