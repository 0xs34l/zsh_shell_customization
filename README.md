Create a file mytheme.zsh-theme in  ~/.oh-my-zsh/custom/themes/
Paste the below code in ~/.oh-my-zsh/custom/themes/mytheme.zsh-theme

PROMPT='%K{#2C5EAC}%F{white}%B %n %b%f%K{#4A90E2}%F{#2C5EAC}%f%F{#000000}%B %m %b%f%K{#F2F2F2}%F{#4A90E2}%f%F{#000000}%B %~ %b%f%K{#000000}%F{#F2F2F2}%f %F{#4A90E2}%B<*>%b%f '

preexec() {
    print
}

first_prompt=1

precmd() {
    if (( first_prompt )); then
        first_prompt=0
    else
        print
    fi
}
