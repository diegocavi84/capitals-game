{\rtf1\ansi\ansicpg1252\cocoartf2867
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 import requests\
import random\
import time\
\
class CapitalGame:\
    def __init__(self):\
        self.score = 0\
        self.played_countries = []\
        self.using_api = True\
        \
    def get_random_country(self):\
        """Gets a random country with multiple fallback strategies"""\
        # Strategy 1: Try specific endpoint\
        if self.using_api:\
            country = self._try_api_specific_endpoint()\
            if country:\
                return country\
            \
            # Strategy 2: Try alternative endpoint\
            country = self._try_api_alternative_endpoint()\
            if country:\
                return country\
            \
            # If both fail, use local data\
            self.using_api = False\
            print("\uc0\u55357 \u56615  Switching to offline mode (local data)...")\
        \
        return self.local_random_country()\
    \
    def _try_api_specific_endpoint(self):\
        """Try with a more specific and simple endpoint"""\
        try:\
            print("\uc0\u55357 \u56599  Connecting to API...")\
            response = requests.get(\
                'https://restcountries.com/v3.1/independent?status=true&fields=name,capital,region,population,languages',\
                timeout=8\
            )\
            \
            if response.status_code == 200:\
                countries = response.json()\
                if countries and len(countries) > 0:\
                    country = self._choose_valid_country(countries)\
                    if country:\
                        print("\uc0\u9989  Connected via API - Specific endpoint")\
                        return country\
            else:\
                print(f"\uc0\u9888 \u65039   HTTP Error \{response.status_code\} in specific endpoint")\
                \
        except Exception as e:\
            print(f"\uc0\u9888 \u65039   Error in specific endpoint: \{type(e).__name__\}")\
            \
        return None\
    \
    def _try_api_alternative_endpoint(self):\
        """Try with an alternative more basic endpoint"""\
        try:\
            print("\uc0\u55357 \u56599  Trying alternative endpoint...")\
            response = requests.get(\
                'https://restcountries.com/v3.1/all?fields=name,capital,region,population,languages',\
                timeout=8\
            )\
            \
            if response.status_code == 200:\
                countries = response.json()\
                if countries and len(countries) > 0:\
                    country = self._choose_valid_country(countries)\
                    if country:\
                        print("\uc0\u9989  Connected via API - Alternative endpoint")\
                        return country\
            else:\
                print(f"\uc0\u9888 \u65039   HTTP Error \{response.status_code\} in alternative endpoint")\
                \
        except Exception as e:\
            print(f"\uc0\u9888 \u65039   Error in alternative endpoint: \{type(e).__name__\}")\
            \
        return None\
    \
    def _choose_valid_country(self, countries):\
        """Choose a valid country that has a capital"""\
        attempts = 0\
        while attempts < 20:\
            country = random.choice(countries)\
            \
            if ('capital' in country and \
                country['capital'] and \
                len(country['capital']) > 0 and \
                country['capital'][0] and\
                'name' in country and\
                'common' in country['name']):\
                \
                country_name = country['name']['common']\
                \
                if (country_name not in self.played_countries or \
                    len(self.played_countries) >= len(countries)):\
                    \
                    self.played_countries.append(country_name)\
                    return country\
            \
            attempts += 1\
        \
        print("\uc0\u9888 \u65039   No valid countries found in API")\
        return None\
    \
    def local_random_country(self):\
        """Extended local data - 25 countries"""\
        local_countries = [\
            \{\
                'name': \{'common': 'France', 'official': 'French Republic'\},\
                'capital': ['Paris'],\
                'region': 'Europe',\
                'population': 67391582,\
                'languages': \{'fra': 'French'\},\
                'fun_fact': "It's the most visited country in the world with over 89 million tourists annually."\
            \},\
            \{\
                'name': \{'common': 'Japan', 'official': 'Japan'\},\
                'capital': ['Tokyo'],\
                'region': 'Asia',\
                'population': 125836021,\
                'languages': \{'jpn': 'Japanese'\},\
                'fun_fact': "Has the highest life expectancy in the world and is the birthplace of sushi."\
            \},\
            \{\
                'name': \{'common': 'Brazil', 'official': 'Federative Republic of Brazil'\},\
                'capital': ['Brasilia'],\
                'region': 'Americas',\
                'population': 212559409,\
                'languages': \{'por': 'Portuguese'\},\
                'fun_fact': "It's the fifth largest country in the world and home to the Amazon rainforest."\
            \},\
            \{\
                'name': \{'common': 'Egypt', 'official': 'Arab Republic of Egypt'\},\
                'capital': ['Cairo'],\
                'region': 'Africa',\
                'population': 102334403,\
                'languages': \{'ara': 'Arabic'\},\
                'fun_fact': "Has the oldest pyramids in the world and ancient pharaonic civilization."\
            \},\
            \{\
                'name': \{'common': 'Australia', 'official': 'Commonwealth of Australia'\},\
                'capital': ['Canberra'],\
                'region': 'Oceania',\
                'population': 25687041,\
                'languages': \{'eng': 'English'\},\
                'fun_fact': "It's both a country and a continent with unique kangaroos."\
            \},\
            \{\
                'name': \{'common': 'Germany', 'official': 'Federal Republic of Germany'\},\
                'capital': ['Berlin'],\
                'region': 'Europe',\
                'population': 83240525,\
                'languages': \{'deu': 'German'\},\
                'fun_fact': "Known for its history, castles, and being a leader in automotive engineering."\
            \},\
            \{\
                'name': \{'common': 'Canada', 'official': 'Canada'\},\
                'capital': ['Ottawa'],\
                'region': 'Americas',\
                'population': 38005238,\
                'languages': \{'eng': 'English', 'fra': 'French'\},\
                'fun_fact': "It's the second largest country in the world and has the longest coastline."\
            \},\
            \{\
                'name': \{'common': 'Italy', 'official': 'Italian Republic'\},\
                'capital': ['Rome'],\
                'region': 'Europe',\
                'population': 59554023,\
                'languages': \{'ita': 'Italian'\},\
                'fun_fact': "Birthplace of the Roman Empire and Renaissance, with more UNESCO sites than any other country."\
            \},\
            \{\
                'name': \{'common': 'Mexico', 'official': 'United Mexican States'\},\
                'capital': ['Mexico City'],\
                'region': 'Americas',\
                'population': 128932753,\
                'languages': \{'spa': 'Spanish'\},\
                'fun_fact': "Has the largest pyramid in the world by volume (Great Pyramid of Cholula)."\
            \},\
            \{\
                'name': \{'common': 'China', 'official': "People's Republic of China"\},\
                'capital': ['Beijing'],\
                'region': 'Asia',\
                'population': 1402112000,\
                'languages': \{'zho': 'Chinese'\},\
                'fun_fact': "Has the longest wall in the world stretching over 21,000 km."\
            \},\
            \{\
                'name': \{'common': 'Spain', 'official': 'Kingdom of Spain'\},\
                'capital': ['Madrid'],\
                'region': 'Europe',\
                'population': 47351567,\
                'languages': \{'spa': 'Spanish'\},\
                'fun_fact': "Hosts the world's second biggest food fight: La Tomatina festival."\
            \},\
            \{\
                'name': \{'common': 'Argentina', 'official': 'Argentine Republic'\},\
                'capital': ['Buenos Aires'],\
                'region': 'Americas',\
                'population': 45376763,\
                'languages': \{'spa': 'Spanish'\},\
                'fun_fact': "It's the largest Spanish-speaking country and birthplace of tango."\
            \},\
            \{\
                'name': \{'common': 'United Kingdom', 'official': 'United Kingdom of Great Britain and Northern Ireland'\},\
                'capital': ['London'],\
                'region': 'Europe',\
                'population': 67215293,\
                'languages': \{'eng': 'English'\},\
                'fun_fact': "Home to the world's most famous royal family and Big Ben clock."\
            \},\
            \{\
                'name': \{'common': 'India', 'official': 'Republic of India'\},\
                'capital': ['New Delhi'],\
                'region': 'Asia',\
                'population': 1380004385,\
                'languages': \{'hin': 'Hindi', 'eng': 'English'\},\
                'fun_fact': "It's the second most populated country and birthplace of yoga."\
            \},\
            \{\
                'name': \{'common': 'Russia', 'official': 'Russian Federation'\},\
                'capital': ['Moscow'],\
                'region': 'Europe',\
                'population': 144104080,\
                'languages': \{'rus': 'Russian'\},\
                'fun_fact': "It's the largest country in the world, spanning two continents."\
            \}\
        ]\
        \
        # Choose non-repeated country if possible\
        available_countries = [c for c in local_countries if c['name']['common'] not in self.played_countries]\
        \
        if not available_countries:\
            # If all used, reset the list\
            self.played_countries.clear()\
            available_countries = local_countries\
        \
        country = random.choice(available_countries)\
        self.played_countries.append(country['name']['common'])\
        return country\
    \
    def show_country_info(self, country):\
        """Shows detailed information about the country"""\
        print(f"\\n\uc0\u55357 \u56481  INFORMATION ABOUT \{country['name']['common'].upper()\}:")\
        print(f"   \uc0\u55357 \u56525  Capital: \{country['capital'][0]\}")\
        print(f"   \uc0\u55356 \u57101  Region: \{country['region']\}")\
        print(f"   \uc0\u55357 \u56421  Population: \{country['population']:,\}")\
        \
        if 'languages' in country:\
            languages = list(country['languages'].values())\
            print(f"   \uc0\u55357 \u56803 \u65039  Languages: \{', '.join(languages)\}")\
        \
        # Fun facts\
        if 'fun_fact' in country:\
            print(f"   \uc0\u55357 \u56589  Fun fact: \{country['fun_fact']\}")\
    \
    def play_round(self):\
        """Plays one round of the game"""\
        country = self.get_random_country()\
        correct_capital = country['capital'][0]\
        \
        print(f"\\n\{'='*50\}")\
        print(f"\uc0\u55356 \u57332  Question #\{len(self.played_countries)\}")\
        print(f"\uc0\u55356 \u57101  Country: \{country['name']['common']\}")\
        print(f"\uc0\u55356 \u57307 \u65039  What is the capital of \{country['name']['common']\}?")\
        \
        attempts = 0\
        max_attempts = 4\
        \
        while attempts < max_attempts:\
            try:\
                if attempts == 0:\
                    answer = input("Your answer: ").strip()\
                else:\
                    answer = input(f"Attempt \{attempts + 1\}/\{max_attempts\}: ").strip()\
                \
                # Allow exit at any time\
                if answer.lower() in ['exit', 'quit', 'stop', 'q']:\
                    return False\
                \
                # More flexible comparison\
                if (answer.lower() == correct_capital.lower() or \
                    self._compare_answer(answer, correct_capital)):\
                    self.score += 1\
                    print(f"\uc0\u9989  Correct! +1 point")\
                    print(f"\uc0\u55356 \u57263  Current score: \{self.score\}")\
                    break\
                else:\
                    attempts += 1\
                    if attempts < max_attempts:\
                        print(f"\uc0\u10060  Incorrect. You have \{max_attempts - attempts\} attempts left")\
                    else:\
                        # Last failed attempt\
                        self.score = max(0, self.score - 1)\
                        print(f"\uc0\u55357 \u56485  No more attempts. -1 point")\
                        print(f"\uc0\u55356 \u57263  Current score: \{self.score\}")\
                        self.show_country_info(country)\
            \
            except KeyboardInterrupt:\
                print("\\n\\n\uc0\u9888 \u65039   Game interrupted by user")\
                return False\
            except Exception as e:\
                print(f"\uc0\u10060  Error: \{e\}")\
                continue\
        \
        return True\
    \
    def _compare_answer(self, answer, correct_capital):\
        """More flexible answer comparison"""\
        # Normalize texts\
        resp = answer.lower().strip()\
        correct = correct_capital.lower().strip()\
        \
        # Special cases\
        variations = \{\
            'mexico city': ['ciudad de mexico', 'cdmx'],\
            'buenos aires': ['bs as', 'buenosaires'],\
            'new delhi': ['nueva delhi', 'delhi'],\
            'washington d.c.': ['washington dc', 'washington'],\
            'santiago': ['santiago de chile'],\
            'lima': ['lima metropolitana'],\
            'bogota': ['bogot\'e1', 'bogota d.c.'],\
            'quito': ['san francisco de quito']\
        \}\
        \
        if correct in variations:\
            if resp in variations[correct] or resp == correct:\
                return True\
        \
        return resp == correct\
    \
    def show_statistics(self):\
        """Shows final game statistics"""\
        print(f"\\n\{'='*50\}")\
        print("\uc0\u55356 \u57262  FINAL STATISTICS")\
        print(f"\uc0\u55357 \u56522  Final score: \{self.score\}")\
        print(f"\uc0\u55356 \u57102  Countries played: \{len(self.played_countries)\}")\
        print(f"\uc0\u55357 \u56615  Mode: \{'API' if self.using_api else 'Local data'\}")\
        \
        if self.score >= 10:\
            print("\uc0\u55356 \u57286  Excellent! You're a geography expert!")\
        elif self.score >= 7:\
            print("\uc0\u55357 \u56397  Very good! You have solid geography knowledge.")\
        elif self.score >= 5:\
            print("\uc0\u55357 \u56490  Well done, but you can improve.")\
        elif self.score >= 3:\
            print("\uc0\u55357 \u56538  Keep practicing, you're on the right track.")\
        else:\
            print("\uc0\u55356 \u57101  Learning geography is fun, keep trying!")\
    \
    def play(self):\
        """Main game function"""\
        print("\uc0\u55356 \u57262  WELCOME TO THE WORLD CAPITALS GAME")\
        print("="*50)\
        print("\uc0\u55357 \u56541  Rules:")\
        print("   \'95 You have 3 attempts to guess each capital")\
        print("   \'95 On the 4th error you lose 1 point")\
        print("   \'95 Each correct answer gives +1 point")\
        print("   \'95 When you fail, you'll see country information")\
        print("   \'95 Type 'exit' to end the game")\
        print("="*50)\
        \
        input("Press Enter to start...")\
        \
        round_num = 0\
        while True:\
            round_num += 1\
            continue_playing = self.play_round()\
            \
            if not continue_playing:\
                break\
            \
            # Ask to continue after each round\
            if round_num >= 1:\
                continue_game = input("\\nWant another question? (y/n): ").strip().lower()\
                if continue_game not in ['y', 'yes', 's', 'si']:\
                    break\
        \
        self.show_statistics()\
\
# Run the game\
if __name__ == "__main__":\
    try:\
        game = CapitalGame()\
        game.play()\
        print("\\n\uc0\u55357 \u56395  Thanks for playing! See you next time.")\
    except KeyboardInterrupt:\
        print("\\n\\n\uc0\u55357 \u56395  Game ended! Thanks for playing.")\
    except Exception as e:\
        print(f"\\n\uc0\u10060  Unexpected error: \{e\}")}