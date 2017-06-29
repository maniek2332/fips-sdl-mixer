cmake_minimum_required(VERSION 2.8.5)

fips_begin_sharedlib(SDL2_mixer)

fips_deps(SDL2)

# TODO support more formats than WAV
add_definitions(-DWAV_MUSIC)

fips_files(
    SDL_mixer/dynamic_flac.c
    SDL_mixer/dynamic_fluidsynth.c
    SDL_mixer/dynamic_mod.c
    SDL_mixer/dynamic_modplug.c
    SDL_mixer/dynamic_mp3.c
    SDL_mixer/dynamic_ogg.c
    SDL_mixer/effect_position.c
    SDL_mixer/effect_stereoreverse.c
    SDL_mixer/effects_internal.c
    SDL_mixer/fluidsynth.c
    SDL_mixer/load_aiff.c
    SDL_mixer/load_flac.c
    SDL_mixer/load_mp3.c
    SDL_mixer/load_ogg.c
    SDL_mixer/load_voc.c
    SDL_mixer/mixer.c
    SDL_mixer/music.c
    SDL_mixer/music_cmd.c
    SDL_mixer/music_flac.c
    SDL_mixer/music_mad.c
    SDL_mixer/music_mod.c
    SDL_mixer/music_modplug.c
    SDL_mixer/music_ogg.c
    SDL_mixer/wavestream.c
)

fips_end_sharedlib()
